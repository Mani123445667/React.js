# React.js
switch component:
I'm trying to build a switch component to toggle the change of dark mode and light mode. I've so far managed to build the switch and allowing it toggle, however, I can't seem to implement the change of background color. I know i will have to set the state with hooks but this is what I have got so far.

Switch Component:

const Switch = ({ isOn, handleToggle }) => {
    return (
        <>
            <input
                checked={isOn}
                onChange={handleToggle}
                className='react-switch-checkbox'
                id={`react-switch-new`}
                type='checkbox'
            />
            <label
                className='react-switch-label'
                htmlFor={`react-switch-new`}
                style={{ background: isOn && '#06D6A0' }}
            >
                <span className={`react-switch-button`} />
            </label>
        </>
    )
}
